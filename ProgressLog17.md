# Progress Log 17

## Overview
Continuing my Internship at ProLab R, I worked on the project - Nimbroll -  Payroll and HR Management System

## Daily Progress Log

## Thursday - 24.9.2026

**Focus: Auth/session fixes, mock login, and the start of page-by-page data mocking**

- Fixed the demo session not surviving a page reload — the logged-in role is now saved to
  `localStorage`, while all mock data (employees, payroll, etc.) still correctly resets to its
  seeded state on every reload.
- Fixed role switching (via the demo role-switcher widget) not redirecting to the correct
  dashboard route for the new role.
- Built a working mock login flow: real email + password fields validated against a set of demo
  accounts, redirecting to the right dashboard on success, with a working sign-out.
- Added mock employee data tied to the demo tenant ("Nimbroll Demo Co."), viewable consistently
  across the Tenant Admin, HR Manager, Payroll Manager, and Employee roles.
- Mocked the Payroll feature end to end: the payroll list, payroll detail view, and the full
  Create Draft → Calculate → Approve → Process workflow.
- Mocked the Leave feature end to end.
- Planned and implemented mock data for Attendance and the employee self-service Attendance page,
  using a "card tap" check-in method in place of biometric/QR device integration.
- Diagnosed and fixed three bugs introduced during the Attendance work.

## Friday - 25.9.2026

**Focus: Finishing the tenant-side demo flow (Dashboard, Payslips, Documents, Reports)**

- Mocked the tenant-side Dashboard, aggregating KPIs from the Payroll, Leave, and Attendance data
  already mocked the day before.
- Mocked the HR Payslips view and finished the employee self-service "My Payslips" page,
  including a year-to-date earnings calculation, and fixed an edge case where that calculation
  could incorrectly show zero.
- Mocked the Documents feature (HR upload/delete) and finished the employee self-service
  "My Documents" page, including a simulated file-upload flow and a working document
  e-signature flow.
- Mocked the Reports page so each of the six report-download buttons generates and downloads a
  real CSV file built from the mocked payroll data, instead of a placeholder action.
- With this, the entire tenant-side demo flow (Tenant Admin, HR Manager, Payroll Manager, and
  Employee roles) is fully functional on mock data, with no dependency on a live backend.
